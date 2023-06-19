# Comparing `tmp/pyappauto-1.0.tar.gz` & `tmp/pyappauto-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyappauto-1.0.tar", last modified: Mon Jun 19 03:25:49 2023, max compression
+gzip compressed data, was "pyappauto-1.0.1.tar", last modified: Mon Jun 19 03:40:55 2023, max compression
```

## Comparing `pyappauto-1.0.tar` & `pyappauto-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 03:25:49.362730 pyappauto-1.0/
--rw-rw-rw-   0        0        0     1088 2023-06-19 03:18:35.000000 pyappauto-1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1530 2023-06-19 03:25:49.362730 pyappauto-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      857 2023-06-19 03:25:08.000000 pyappauto-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 03:25:49.355684 pyappauto-1.0/pyappauto/
--rw-rw-rw-   0        0        0    15230 2023-06-19 03:17:35.000000 pyappauto-1.0/pyappauto/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:25:49.361722 pyappauto-1.0/pyappauto/utils/
--rw-rw-rw-   0        0        0      229 2023-06-19 01:57:47.000000 pyappauto-1.0/pyappauto/utils/errors.py
--rw-rw-rw-   0        0        0     3736 2023-06-19 02:11:18.000000 pyappauto-1.0/pyappauto/utils/keys.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:25:49.359698 pyappauto-1.0/pyappauto.egg-info/
--rw-rw-rw-   0        0        0     1530 2023-06-19 03:25:49.000000 pyappauto-1.0/pyappauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-06-19 03:25:49.000000 pyappauto-1.0/pyappauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 03:25:49.000000 pyappauto-1.0/pyappauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-06-19 03:25:49.000000 pyappauto-1.0/pyappauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-19 03:25:49.000000 pyappauto-1.0/pyappauto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 03:25:49.363736 pyappauto-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1048 2023-06-19 03:24:10.000000 pyappauto-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:40:55.051329 pyappauto-1.0.1/
+-rw-rw-rw-   0        0        0     1088 2023-06-19 03:18:35.000000 pyappauto-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1532 2023-06-19 03:40:55.051329 pyappauto-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      857 2023-06-19 03:25:08.000000 pyappauto-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 03:40:55.044281 pyappauto-1.0.1/pyappauto/
+-rw-rw-rw-   0        0        0    15265 2023-06-19 03:39:04.000000 pyappauto-1.0.1/pyappauto/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:40:55.049317 pyappauto-1.0.1/pyappauto/utils/
+-rw-rw-rw-   0        0        0      229 2023-06-19 01:57:47.000000 pyappauto-1.0.1/pyappauto/utils/errors.py
+-rw-rw-rw-   0        0        0     3736 2023-06-19 02:11:18.000000 pyappauto-1.0.1/pyappauto/utils/keys.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:40:55.048812 pyappauto-1.0.1/pyappauto.egg-info/
+-rw-rw-rw-   0        0        0     1532 2023-06-19 03:40:55.000000 pyappauto-1.0.1/pyappauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-06-19 03:40:55.000000 pyappauto-1.0.1/pyappauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 03:40:55.000000 pyappauto-1.0.1/pyappauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-19 03:40:55.000000 pyappauto-1.0.1/pyappauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-19 03:40:55.000000 pyappauto-1.0.1/pyappauto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 03:40:55.051329 pyappauto-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2023-06-19 03:38:34.000000 pyappauto-1.0.1/setup.py
```

### Comparing `pyappauto-1.0/LICENSE.txt` & `pyappauto-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyappauto-1.0/PKG-INFO` & `pyappauto-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappauto
-Version: 1.0
+Version: 1.0.1
 Summary: Control an app without disturbing your everyday life.
 Home-page: https://github.com/User00092/PyAppAuto
 Author: User0092
 Author-email: unknownuser0092@protonmail.com
 License: MIT
 Keywords: Windows App control,App controller,PyAppAuto
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyappauto-1.0/README.md` & `pyappauto-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyappauto-1.0/pyappauto/__init__.py` & `pyappauto-1.0.1/pyappauto/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-import utils.errors
+import pyappauto.utils.errors
 
 from threading import Thread
 import pygetwindow as gw
 import numpy as np
 import subprocess
 import win32con
 import win32gui
 import win32api
 import win32ui
 import time
 import cv2
 import os
 
+__version__ = '1.0.1'
+
 
 class Instance:
     def __init__(self, hwnd: int | None = None, debug: bool = False):
         """This is the constructor method for the class "Instance"
 
         Args:
             hwnd (int | None, optional): represents the handle to a window. Defaults to None.
```

### Comparing `pyappauto-1.0/pyappauto/utils/keys.py` & `pyappauto-1.0.1/pyappauto/utils/keys.py`

 * *Files identical despite different names*

### Comparing `pyappauto-1.0/pyappauto.egg-info/PKG-INFO` & `pyappauto-1.0.1/pyappauto.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappauto
-Version: 1.0
+Version: 1.0.1
 Summary: Control an app without disturbing your everyday life.
 Home-page: https://github.com/User00092/PyAppAuto
 Author: User0092
 Author-email: unknownuser0092@protonmail.com
 License: MIT
 Keywords: Windows App control,App controller,PyAppAuto
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyappauto-1.0/setup.py` & `pyappauto-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION = "\n" + fh.read()
 
-VERSION = '1.0'
 DESCRIPTION = 'Control an app without disturbing your everyday life.'
 
 # Setting up
 setup(
 	name="pyappauto",
 	url="https://github.com/User00092/PyAppAuto",
-	version=VERSION,
+	version='1.0.1',
 	license='MIT',
 	author="User0092",
 	author_email="unknownuser0092@protonmail.com",
 	description=DESCRIPTION,
 	long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
 	keywords=['Windows App control', 'App controller', 'PyAppAuto'],
```

