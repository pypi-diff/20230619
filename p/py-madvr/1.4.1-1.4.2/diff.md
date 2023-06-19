# Comparing `tmp/py_madvr-1.4.1.tar.gz` & `tmp/py_madvr-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.4.1.tar", last modified: Sun May 14 20:42:14 2023, max compression
+gzip compressed data, was "py_madvr-1.4.2.tar", last modified: Mon Jun 19 16:10:06 2023, max compression
```

## Comparing `py_madvr-1.4.1.tar` & `py_madvr-1.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:42:14.495768 py_madvr-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 20:42:03.000000 py_madvr-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-14 20:42:14.495768 py_madvr-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-14 20:42:03.000000 py_madvr-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:42:14.491768 py_madvr-1.4.1/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 20:42:03.000000 py_madvr-1.4.1/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 20:42:03.000000 py_madvr-1.4.1/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 20:42:03.000000 py_madvr-1.4.1/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-05-14 20:42:03.000000 py_madvr-1.4.1/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:42:14.495768 py_madvr-1.4.1/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-14 20:42:14.000000 py_madvr-1.4.1/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 20:42:14.000000 py_madvr-1.4.1/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:42:14.000000 py_madvr-1.4.1/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 20:42:14.000000 py_madvr-1.4.1/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 20:42:14.495768 py_madvr-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-14 20:42:03.000000 py_madvr-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:42:14.495768 py_madvr-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 20:42:03.000000 py_madvr-1.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 20:42:03.000000 py_madvr-1.4.1/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:10:06.774314 py_madvr-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-19 16:09:55.000000 py_madvr-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-19 16:10:06.774314 py_madvr-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-19 16:09:55.000000 py_madvr-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:10:06.770314 py_madvr-1.4.2/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-19 16:09:55.000000 py_madvr-1.4.2/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-19 16:09:55.000000 py_madvr-1.4.2/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-19 16:09:55.000000 py_madvr-1.4.2/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-06-19 16:09:55.000000 py_madvr-1.4.2/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:10:06.770314 py_madvr-1.4.2/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-19 16:10:06.000000 py_madvr-1.4.2/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-19 16:10:06.000000 py_madvr-1.4.2/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:10:06.000000 py_madvr-1.4.2/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 16:10:06.000000 py_madvr-1.4.2/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 16:10:06.774314 py_madvr-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-19 16:09:55.000000 py_madvr-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:10:06.774314 py_madvr-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:09:55.000000 py_madvr-1.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-19 16:09:55.000000 py_madvr-1.4.2/tests/testMadVR.py
```

### Comparing `py_madvr-1.4.1/LICENSE` & `py_madvr-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.4.1/PKG-INFO` & `py_madvr-1.4.2/py_madvr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py_madvr
-Version: 1.4.1
+Name: py-madvr
+Version: 1.4.2
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.4.1/madvr/commands.py` & `py_madvr-1.4.2/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.4.1/madvr/madvr.py` & `py_madvr-1.4.2/madvr/madvr.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,21 +63,24 @@
         async with self.writer_lock:
             try:
                 self.writer.close()
                 await self.writer.wait_closed()
             except AttributeError:
                 # means its already closed
                 pass
-
+        self.logger.debug("self.writer is closed")
         self.reader = None
         self.is_closed = True
+        self.logger.debug("clearing connection event")
         self.connection_event.clear()
 
         # Clear attr
+        self.logger.debug("clearing attr")
         await self._clear_attr()
+        self.logger.debug("connection is closed")
 
     async def open_connection(self) -> None:
         """Open a connection"""
         self.logger.debug("Starting open connection")
         try:
             await self._reconnect()
         except AckError as err:
@@ -395,18 +398,23 @@
         It uses about 30w idle on standby. I use IR via harmony to turn it on
 
         standby: bool -> standby instead of poweroff if true
         """
         # dont do anything if its off besides mark it off
         # sending command will open connection
         try:
+            # stop trying to reconnect
+            self.logger.debug("setting stop reconnect")
+            self.stop()
+            self.logger.debug("sending power off command")
             res = await self.send_command(["Standby"] if standby else ["PowerOff"])
+            self.logger.debug("closing connection")
             await self.close_connection()
             self.is_on = False
-
+            self.logger.debug("finished power_off")
             return res
 
         except RetryExceededError:
             return "Retries Exceeded"
 
     def print_commands(self) -> str:
         """
```

### Comparing `py_madvr-1.4.1/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.4.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py-madvr
-Version: 1.4.1
+Name: py_madvr
+Version: 1.4.2
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.4.1/setup.py` & `py_madvr-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.4.1",
+    version="1.4.2",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.4.1/tests/testMadVR.py` & `py_madvr-1.4.2/tests/testMadVR.py`

 * *Files identical despite different names*

