# Comparing `tmp/amqp-mqtt-transport-0.1.0.tar.gz` & `tmp/amqp-mqtt-transport-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqp-mqtt-transport-0.1.0.tar", last modified: Mon Jun 19 13:08:14 2023, max compression
+gzip compressed data, was "amqp-mqtt-transport-0.1.1.tar", last modified: Mon Jun 19 13:41:43 2023, max compression
```

## Comparing `amqp-mqtt-transport-0.1.0.tar` & `amqp-mqtt-transport-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:08:14.788526 amqp-mqtt-transport-0.1.0/
--rw-r--r--   0 igor      (1001) igor      (1001)       87 2023-06-19 12:04:53.000000 amqp-mqtt-transport-0.1.0/.gitattributes
--rw-r--r--   0 igor      (1001) igor      (1001)      483 2023-06-19 12:04:52.000000 amqp-mqtt-transport-0.1.0/.gitignore
--rw-rw-r--   0 igor      (1001) igor      (1001)     1072 2023-06-19 12:17:58.000000 amqp-mqtt-transport-0.1.0/LICENSE
--rw-rw-r--   0 igor      (1001) igor      (1001)     1129 2023-06-19 13:07:42.000000 amqp-mqtt-transport-0.1.0/Makefile
--rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-19 13:08:14.788526 amqp-mqtt-transport-0.1.0/PKG-INFO
--rw-r--r--   0 igor      (1001) igor      (1001)      788 2023-06-19 13:04:30.000000 amqp-mqtt-transport-0.1.0/README.md
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:08:14.760525 amqp-mqtt-transport-0.1.0/amqp_mqtt_transport.egg-info/
--rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-19 13:08:14.000000 amqp-mqtt-transport-0.1.0/amqp_mqtt_transport.egg-info/PKG-INFO
--rw-rw-r--   0 igor      (1001) igor      (1001)      605 2023-06-19 13:08:14.000000 amqp-mqtt-transport-0.1.0/amqp_mqtt_transport.egg-info/SOURCES.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)        1 2023-06-19 13:08:14.000000 amqp-mqtt-transport-0.1.0/amqp_mqtt_transport.egg-info/dependency_links.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)       92 2023-06-19 13:08:14.000000 amqp-mqtt-transport-0.1.0/amqp_mqtt_transport.egg-info/requires.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)       10 2023-06-19 13:08:14.000000 amqp-mqtt-transport-0.1.0/amqp_mqtt_transport.egg-info/top_level.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)      799 2023-06-19 12:46:20.000000 amqp-mqtt-transport-0.1.0/pyproject.toml
--rw-rw-r--   0 igor      (1001) igor      (1001)       91 2023-06-19 12:31:08.000000 amqp-mqtt-transport-0.1.0/requirements.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)       38 2023-06-19 13:08:14.788526 amqp-mqtt-transport-0.1.0/setup.cfg
--rw-rw-r--   0 igor      (1001) igor      (1001)       37 2023-06-19 12:41:38.000000 amqp-mqtt-transport-0.1.0/setup.py
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:08:14.768525 amqp-mqtt-transport-0.1.0/transport/
--rw-rw-r--   0 igor      (1001) igor      (1001)      146 2023-06-19 12:15:25.000000 amqp-mqtt-transport-0.1.0/transport/__init__.py
--rw-rw-r--   0 igor      (1001) igor      (1001)      956 2023-06-19 12:15:26.000000 amqp-mqtt-transport-0.1.0/transport/abc.py
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:08:14.780525 amqp-mqtt-transport-0.1.0/transport/amqp/
--rw-rw-r--   0 igor      (1001) igor      (1001)       75 2023-06-19 12:15:27.000000 amqp-mqtt-transport-0.1.0/transport/amqp/__init__.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     1728 2023-06-19 12:15:27.000000 amqp-mqtt-transport-0.1.0/transport/amqp/consumer.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     5533 2023-06-19 12:15:29.000000 amqp-mqtt-transport-0.1.0/transport/amqp/controller.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     1521 2023-06-19 12:15:30.000000 amqp-mqtt-transport-0.1.0/transport/amqp/publisher.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     2102 2023-06-19 12:15:26.000000 amqp-mqtt-transport-0.1.0/transport/message_scheduler.py
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:08:14.788526 amqp-mqtt-transport-0.1.0/transport/mqtt/
--rw-rw-r--   0 igor      (1001) igor      (1001)       51 2023-06-19 12:15:30.000000 amqp-mqtt-transport-0.1.0/transport/mqtt/__init__.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     3115 2023-06-19 12:15:31.000000 amqp-mqtt-transport-0.1.0/transport/mqtt/controller.py
--rw-rw-r--   0 igor      (1001) igor      (1001)      807 2023-06-19 12:15:32.000000 amqp-mqtt-transport-0.1.0/transport/mqtt/publisher.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     2430 2023-06-19 12:15:27.000000 amqp-mqtt-transport-0.1.0/transport/scheduled_publisher.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:41:43.859039 amqp-mqtt-transport-0.1.1/
+-rw-r--r--   0 igor      (1001) igor      (1001)       87 2023-06-19 12:04:53.000000 amqp-mqtt-transport-0.1.1/.gitattributes
+-rw-r--r--   0 igor      (1001) igor      (1001)      483 2023-06-19 12:04:52.000000 amqp-mqtt-transport-0.1.1/.gitignore
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1072 2023-06-19 12:17:58.000000 amqp-mqtt-transport-0.1.1/LICENSE
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1012 2023-06-19 13:15:40.000000 amqp-mqtt-transport-0.1.1/Makefile
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-19 13:41:43.859039 amqp-mqtt-transport-0.1.1/PKG-INFO
+-rw-r--r--   0 igor      (1001) igor      (1001)      788 2023-06-19 13:04:30.000000 amqp-mqtt-transport-0.1.1/README.md
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:41:43.835038 amqp-mqtt-transport-0.1.1/amqp_mqtt_transport.egg-info/
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-19 13:41:43.000000 amqp-mqtt-transport-0.1.1/amqp_mqtt_transport.egg-info/PKG-INFO
+-rw-rw-r--   0 igor      (1001) igor      (1001)      588 2023-06-19 13:41:43.000000 amqp-mqtt-transport-0.1.1/amqp_mqtt_transport.egg-info/SOURCES.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)        1 2023-06-19 13:41:43.000000 amqp-mqtt-transport-0.1.1/amqp_mqtt_transport.egg-info/dependency_links.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)       92 2023-06-19 13:41:43.000000 amqp-mqtt-transport-0.1.1/amqp_mqtt_transport.egg-info/requires.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)       10 2023-06-19 13:41:43.000000 amqp-mqtt-transport-0.1.1/amqp_mqtt_transport.egg-info/top_level.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)      799 2023-06-19 13:40:21.000000 amqp-mqtt-transport-0.1.1/pyproject.toml
+-rw-rw-r--   0 igor      (1001) igor      (1001)       38 2023-06-19 13:41:43.859039 amqp-mqtt-transport-0.1.1/setup.cfg
+-rw-rw-r--   0 igor      (1001) igor      (1001)       37 2023-06-19 12:41:38.000000 amqp-mqtt-transport-0.1.1/setup.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:41:43.839038 amqp-mqtt-transport-0.1.1/transport/
+-rw-rw-r--   0 igor      (1001) igor      (1001)      146 2023-06-19 12:15:25.000000 amqp-mqtt-transport-0.1.1/transport/__init__.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)      956 2023-06-19 12:15:26.000000 amqp-mqtt-transport-0.1.1/transport/abc.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:41:43.847039 amqp-mqtt-transport-0.1.1/transport/amqp/
+-rw-rw-r--   0 igor      (1001) igor      (1001)       75 2023-06-19 12:15:27.000000 amqp-mqtt-transport-0.1.1/transport/amqp/__init__.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1728 2023-06-19 12:15:27.000000 amqp-mqtt-transport-0.1.1/transport/amqp/consumer.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     5533 2023-06-19 12:15:29.000000 amqp-mqtt-transport-0.1.1/transport/amqp/controller.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1521 2023-06-19 12:15:30.000000 amqp-mqtt-transport-0.1.1/transport/amqp/publisher.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     2102 2023-06-19 12:15:26.000000 amqp-mqtt-transport-0.1.1/transport/message_scheduler.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:41:43.859039 amqp-mqtt-transport-0.1.1/transport/mqtt/
+-rw-rw-r--   0 igor      (1001) igor      (1001)       51 2023-06-19 12:15:30.000000 amqp-mqtt-transport-0.1.1/transport/mqtt/__init__.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     3115 2023-06-19 12:15:31.000000 amqp-mqtt-transport-0.1.1/transport/mqtt/controller.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)      807 2023-06-19 12:15:32.000000 amqp-mqtt-transport-0.1.1/transport/mqtt/publisher.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     2430 2023-06-19 12:15:27.000000 amqp-mqtt-transport-0.1.1/transport/scheduled_publisher.py
```

### Comparing `amqp-mqtt-transport-0.1.0/LICENSE` & `amqp-mqtt-transport-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.0/Makefile` & `amqp-mqtt-transport-0.1.1/Makefile`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 define HELP_MSG
 Makefile for python project
 Avaliable commands:
 venv - creates python virtual environment
-init - create venv and install dependencies from requirements.txt
-install - install this package to venv
+install - install this package and its dependencies to venv
 build - build package and tar it
 upload_to_pypi - build and upload to pypi repository
 clean - clean all intermediate build files as well as dist tar files
 autopep8 - run autopep8 linter and change files
 help - prints this message
 endef
 
 venv:
 	test -d venv || python3.10 -m venv venv
 
-init: venv
-	. venv/bin/activate && pip install -r requirements.txt
-
 run: venv
 	@echo "This is import only package, can't run"
 
-install: venv init
+install: venv
 	. venv/bin/activate && python3.10 -m pip install -e .
 
-build: init
+build: install
 	. venv/bin/activate && python3.10 -m build
 
 upload_to_pypi: build
 	. venv/bin/activate && python3.10 -m twine upload --repository pypi dist/*
 
-autopep8: init
+autopep8: install
 	. venv/bin/activate && autopep8 --in-place --exclude "./venv/**" --recursive .
 
 clean:
 	rm -rf venv dist *.egg-info
 	find -iname "*.pyc" -delete
 
 export HELP_MSG
 help:
 	@echo "$$HELP_MSG"
 
-.PHONY: init venv install clean run build upload_to_pypi autopep8 help
+.PHONY: venv install clean run build upload_to_pypi autopep8 help
```

### Comparing `amqp-mqtt-transport-0.1.0/PKG-INFO` & `amqp-mqtt-transport-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqp-mqtt-transport
-Version: 0.1.0
+Version: 0.1.1
 Summary: Small wrapper for pykka-amqp and paho-mqtt packages. Makes it easier to create consumers/publishers
 Author-email: Igor Toropov <it.cups.54@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `amqp-mqtt-transport-0.1.0/README.md` & `amqp-mqtt-transport-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.0/amqp_mqtt_transport.egg-info/PKG-INFO` & `amqp-mqtt-transport-0.1.1/amqp_mqtt_transport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqp-mqtt-transport
-Version: 0.1.0
+Version: 0.1.1
 Summary: Small wrapper for pykka-amqp and paho-mqtt packages. Makes it easier to create consumers/publishers
 Author-email: Igor Toropov <it.cups.54@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `amqp-mqtt-transport-0.1.0/amqp_mqtt_transport.egg-info/SOURCES.txt` & `amqp-mqtt-transport-0.1.1/amqp_mqtt_transport.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 .gitattributes
 .gitignore
 LICENSE
 Makefile
 README.md
 pyproject.toml
-requirements.txt
 setup.py
 amqp_mqtt_transport.egg-info/PKG-INFO
 amqp_mqtt_transport.egg-info/SOURCES.txt
 amqp_mqtt_transport.egg-info/dependency_links.txt
 amqp_mqtt_transport.egg-info/requires.txt
 amqp_mqtt_transport.egg-info/top_level.txt
 transport/__init__.py
```

### Comparing `amqp-mqtt-transport-0.1.0/pyproject.toml` & `amqp-mqtt-transport-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amqp-mqtt-transport"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Igor Toropov", email="it.cups.54@gmail.com" },
 ]
 description = "Small wrapper for pykka-amqp and paho-mqtt packages. Makes it easier to create consumers/publishers"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "tenacity==8.0.1",
+    "tenacity<=8.2.2",
     "aio-pika==8.2.5",
     "autopep8==2.0.2",
     "paho-mqtt==1.5.1",
     "build==0.10.0",
     "twine==4.0.2"
 ]
```

### Comparing `amqp-mqtt-transport-0.1.0/transport/abc.py` & `amqp-mqtt-transport-0.1.1/transport/abc.py`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.0/transport/amqp/consumer.py` & `amqp-mqtt-transport-0.1.1/transport/amqp/consumer.py`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.0/transport/amqp/controller.py` & `amqp-mqtt-transport-0.1.1/transport/amqp/controller.py`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.0/transport/amqp/publisher.py` & `amqp-mqtt-transport-0.1.1/transport/amqp/publisher.py`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.0/transport/message_scheduler.py` & `amqp-mqtt-transport-0.1.1/transport/message_scheduler.py`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.0/transport/mqtt/controller.py` & `amqp-mqtt-transport-0.1.1/transport/mqtt/controller.py`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.0/transport/mqtt/publisher.py` & `amqp-mqtt-transport-0.1.1/transport/mqtt/publisher.py`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.0/transport/scheduled_publisher.py` & `amqp-mqtt-transport-0.1.1/transport/scheduled_publisher.py`

 * *Files identical despite different names*

